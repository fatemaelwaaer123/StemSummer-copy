# third_party/StemSummer

This path is intended to contain the GraysonC2/StemSummer repository as a git submodule.

I added a .gitmodules entry and this placeholder README on the branch `add-submodule-StemSummer`.

Important: GitHub's file API cannot create the special gitlink entry (mode 160000) that records the submodule commit. To fully register the submodule in the repository history you can either:

- Initialize the submodule locally and push the branch from your machine (recommended):

  git clone git@github.com:fatemaelwaaer123/StemSummer-copy.git
  cd StemSummer-copy
  git checkout -b add-submodule-StemSummer origin/add-submodule-StemSummer
  git submodule add git@github.com:GraysonC2/StemSummer.git third_party/StemSummer
  git commit -m "Add GraysonC2/StemSummer as submodule"
  git push -u origin add-submodule-StemSummer

- Or, if you want me to, I can try to add a gitlink commit for you (this requires additional repo-level operations). Tell me if you want me to proceed with that.

After the submodule is properly added, users should run:

  git submodule update --init --recursive

