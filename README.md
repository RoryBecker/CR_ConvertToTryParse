CR_ConvertToTryParse
====================
Replaces the use of Int.Parse with Int.TryParse

Specifically, will translate 

    int Parsed = Int32.Parse("23");

into 

    Int32 Parsed;
    bool Success = Int32.TryParse("23", out Parsed);

Usage
===
Place the caret on the '=' sign, and activate the "Convert to TryParse" Refactoring.
