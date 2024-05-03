Hi! I'm Mary Ann “Mara” Estopin, a Fraud Specialist at JP Morgan and Co., currently loaned to Retail Customer Service to support their line of business.

- **About Me**: I am a dedicated professional with a strong background in fraud detection and prevention. I am known for my analytical thinking skills, attention to detail, critical thinking, and problem-solving abilities. I thrive in teamwork and collaboration, and I uphold professionalism and a strong work ethic in all that I do.

- **Skills**:
  - Analytical thinking skills
  - Attention to details
  - Critical thinking and problem-solving skill
  - Teamwork and collaboration
  - Professionalism and strong work ethic
  - Oral and written communication skills
  - Leadership

- **Interests**: I am currently studying Data Science and learning various programming languages such as HTML, CSS, JavaScript, Python, R, and SQL. I am passionate about leveraging data and technology to drive insights and solve complex problems.

- **Contact**:
  - Email: estopin.maryann06@gmail.com
  - LinkedIn: [LinkedIn Profile](https://www.linkedin.com/in/mary-ann-estopin-a7b9a8a3/)

Feel free to reach out for collaborations or just to say hi! 😊


import requests

username = 'your_github_username'
token = 'your_github_token'

url = 'https://api.github.com/user/repos'

headers = {
    'Authorization': 'token ' + token
}

data = {
    'name': 'new-repository',
    'description': 'This is a new repository created using the GitHub API',
    'private': False
}

response = requests.post(url, json=data, headers=headers)

if response.status_code == 201:
    print('Repository created successfully')
else:
    print('Failed to create repository')
    print(response.json())