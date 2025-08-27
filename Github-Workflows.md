- A workflow is a configurable automated process that will run one job or more jobs. Defined in YAML file.
- Defined in .github/workflows directory.
- Repo can contain multiple repos
- name property defines and easily identifies the workflow.

- Workflow triggers are events that cause a workflow to run.
- Events that occur in your workflows repo
- Events that occur outside of Github and trigger a repository_dispatch event on Github
- SCheduled times.
- Manual

## Workflow components

- Actions : Reusable units of code that performs specific job and can be combined to create workflows.
- Workflows: Automated process defined in your repo that coordinates one or more jobs, triggered by events or on a schedule.
- Jobs : A set of steps that execute on the same runner. Each job is run in its own virtual environment parallel unless configured otherwise.
- Steps : Individual task within a job that run commands or actions sequentially.
- Runs : A single instance of a workflow execution triggered by events, representing the complete run-through of a workflow.
- Runners : The servers that host the environment where jobs are execued, available as Github-hosted or self-hosted options.
- Marketplace : A place to discover and share reusable actions, enhancing workflow capabablilities with community-developed tools.

## Triggers

- Schedule can usa cron expression to trigger a workflow ata a specific time or day.
- on: 
  schedule:
    - cron: '0 0 * * *' # At midnight every day
    - cron: '0 12 * * *' # At noon every day

    jobs: 


