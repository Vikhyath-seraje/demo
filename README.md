ssh-keygen -t ed25519 -C "gowdanjan18@gmail.com"
 cat ~/.ssh/id_ed25519.pub
 eval "$(ssh-agent -s)"
 ssh-add ~/.ssh/id_ed25519
 ssh -T git@github.com
 mkdir demo
cd demo
git init
echo "Hello Git" > a.txt
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/AnjanC18/demo.git
git push -u origin main
