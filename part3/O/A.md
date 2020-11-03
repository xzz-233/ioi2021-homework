我们考虑任选一点为根，接下来易见一个贪心：自底向上，尽量选出一条路径。但问题在于有很多种选法，我们还需考虑有可能有一条路径要留给更祖先处的合并，而在一个节点处的情况则是一般图匹配，我们只需处理出在最大匹配中有哪些点可以不被匹配就可以了。我的带花树板子是 $O(nm)$ 的，那么在这道题因为只需要在每个点处做度数大小的匹配，复杂度不超过 $O(n^2 + nd^2)$。