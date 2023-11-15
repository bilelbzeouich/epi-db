select emp, last_name, department_id
from hr.employees
where department_id in (10, 20, 30)
order by department_id;

select emp, last_name, department_id, department_name
from hr.employees
join hr.departments
on employees.department_id = departments.department_id;
