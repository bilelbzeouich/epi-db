select emp, last_name, department_id
from hr.employees
where department_id in (10, 20, 30)
order by department_id;
