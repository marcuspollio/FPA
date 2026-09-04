## Summary of Activities - OCCT Liaison - August 2026

### Weekly OCCT Dev meeting

We've had weekly OCCT Dev meetings on 2, 16, 23, and 30 August.

The meetings work well, many things are discussed, such as fillets, seams,
release cycles, etc.  Dmitrii is writing blog posts about relevant topics for
us, such as on
[B-splines](https://occt3d.com/blog/bspline-bezier-evaluation-in-occt/).

### Fillet issues

As discussed in the last meeting, it is useful for Dmitrii to have as much as
possible fillet issues.  I've submitted:

- [#1421](https://github.com/Open-Cascade-SAS/OCCT/issues/1421)
- [#1427](https://github.com/Open-Cascade-SAS/OCCT/issues/1427)
- [#1430](https://github.com/Open-Cascade-SAS/OCCT/issues/1430), which had 5
  different issues.

I have been working on
[#16644](https://github.com/FreeCAD/FreeCAD/issues/16644) but it hasn't been
completed.

### Adapt FreeCAD to OCCT 8.1-dev

Because of changes in OCCT, FreeCAD doesn't compile on OCCT 8.1.  In
collaboration with Dmitrii this has been fixed.  Currently no PR is necessary,
because it unclear what of these changes will make it to the actual 8.1
release.

### Allow `-Werror` with OCCT 8 in FreeCAD

Since the Pixi builds will be build with `-Werror`, it is necessary to adapt
FreeCAD to OCCT 8 which contains many deprecations.  I've updated [PR
#30940](https://github.com/FreeCAD/FreeCAD/pull/30940) and it is now merged.

