# Haskell Maybe Type Pattern Matching Error
This repository demonstrates a common error in Haskell programming related to pattern matching on the `Maybe` type.  The `bug.hs` file contains code that incorrectly handles the `Maybe` type, leading to a runtime error or a compiler warning about non-exhaustive patterns. The `bugSolution.hs` file provides the corrected version.

**Problem:** The original code fails to handle the `Nothing` case when pattern matching on a `Maybe` value. This leads to incomplete pattern matching and causes a runtime error if `Nothing` is encountered.  It is a common mistake for new Haskell programmers to miss this case, as the default behaviour of pattern matching will not work in this instance.

**Solution:** The corrected version explicitly handles both the `Just` and `Nothing` cases, providing a complete pattern match and preventing any runtime errors.