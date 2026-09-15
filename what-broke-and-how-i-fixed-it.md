\# What Broke and How I Fixed It



During the setup, some tools were initially unavailable on my system. The GitHub CLI and AWS CLI commands were not recognized, so I installed them using Windows Package Manager (winget). AWS CLI authentication initially failed because no credentials were configured, so I used aws login to authenticate my AWS account. Python 3.12 was installed through uv, but py -3.12 did not recognize the uv-managed installation, so I verified Python 3.12.13 using uv run --python 3.12 python --version. These issues helped me understand that installing a tool and verifying that it actually works are two different steps.

