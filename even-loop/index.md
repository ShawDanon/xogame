事件循环（even loop）
主线程任务执行完->执行微任务队列所有事件，如果事件中有宏任务就推到宏任务队列，如果有微任务就推到微任务队列最后，这个刚推的微任务也会执行，直到当前事件循环中没有微任务了才进行下一步->宏任务队列（把第一个宏任务放入主线程进行执行）->循环