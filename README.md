# queuerev
queue<int> rev(queue<int> q)
{
    // add code here.
    stack<int>s;
    while(!q.empty())
    {
        s.push(q.front());
        q.pop();
        
    }
    queue<int>q1;
    while(!s.empty())
    {
        q1.push(s.top());
        s.pop();
        
    }
    return q1;
}
