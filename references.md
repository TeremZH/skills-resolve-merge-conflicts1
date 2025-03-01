FUNCTION pkg_fn_get_sname
(p_sid number)
RETURN varchar2
IS
v_sname        varchar2 (50);
BEGIN
SELECT        SName
INTO               v_sname
FROM             MM_Student
WHERE         Sid = p_sid;
RETURN v_sname;
END pkg_fn_get_sname;
END pkg_student;
/
SHOW ERRORS;
