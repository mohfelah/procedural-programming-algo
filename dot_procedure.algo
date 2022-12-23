PROCEDURE dot_product(v1, v2 : ARRAY_OF FLOAT, VAR ps : FLOAT)
VAR
    i : INTEGER
BEGIN
    ps := 0;
    i := 0;
    IF (v1.length <> v2.length) THEN
        Write("Vectors with different sizes. We cannot calculate dot product.");
        ps := NAN
    END_IF
    WHILE (i < v1.length) DO
        ps := ps + v1[i]*v2[i];
    END_WHILE
END

ALGORITHM orthogonal_vectors
VAR
    v1, v2 : ARRAY_OF FLOAT;
    ps : FLOAT;
    i, n : INTEGER;
BEGIN
    i := 0;

    Write("Write v1 and v2 length.")
    Read(n);
    FOR i FROM 0 TO n-1 STEP 1 DO
        Read(v1[i]);
    END_FOR
    FOR i FROM 0 TO n-1 STEP 1 DO
        Read(v2[i]);
    END_FOR

    dot_product(v1, v2, ps)

    IF (ps = 0) THEN
        Write("V1 and V2 are orthogonal")
    ELSE
        Write("V1 and V2 are not orthogonal")
    END_IF
END