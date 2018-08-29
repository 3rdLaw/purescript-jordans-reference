# Effect, Eff, and Aff

## Some History

Before the `0.12.0` release, the `Effect` monad used to be called `Eff`. You can read more about that decision making process [here](https://purescript-resources.readthedocs.io/en/latest/eff-to-effect.html).

In short, the decision was made to drop `Eff`'s "extensible effects". Presumably, to prevent code breakage, `Eff` and package location in imports was unchanged. Rather, it can now be found in the  [purescript-eff](https://pursuit.purescript.org/packages/purescript-eff/3.2.1) package.

One can use either `Effect` or `Eff` for their native effect monad. The `Aff` monad was introduced and in use before this decision was made. Thus,  history explains the naming behind `Aff`: if `Eff` was for synchronous **eff**ects, then `Aff` is for **a**sychronous e**ff**ects.

## Scope of This Folder

If one is curious about `Eff`, read through [the related section](https://leanpub.com/purescript/read#leanpub-auto-the-eff-monad-1) in the "Purescript by Example" book as it won't be covered here.

Since `Effect` has already been explained. our focus will be on `Aff` and its relation and usage with `Effect`. In this folder, we'll peel back the covers of `Node.ReadLine.CleanerInterface` and cover more of `Aff`.