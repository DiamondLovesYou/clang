set(LLVM_LINK_COMPONENTS
  Support
  )

add_clang_library(clangAnalysis
  AnalysisDeclContext.cpp
  BodyFarm.cpp
  CFG.cpp
  CFGReachabilityAnalysis.cpp
  CFGStmtMap.cpp
  CallGraph.cpp
  CloneDetection.cpp
  CocoaConventions.cpp
  ConstructionContext.cpp
  Consumed.cpp
  CodeInjector.cpp
  Dominators.cpp
  ExprMutationAnalyzer.cpp
  FormatString.cpp
  LiveVariables.cpp
  OSLog.cpp
  ObjCNoReturn.cpp
  PostOrderCFGView.cpp
  PrintfFormatString.cpp
  ProgramPoint.cpp
  ReachableCode.cpp
  ScanfFormatString.cpp
  ThreadSafety.cpp
  ThreadSafetyCommon.cpp
  ThreadSafetyLogical.cpp
  ThreadSafetyTIL.cpp
  UninitializedValues.cpp

  LINK_LIBS
  clangAST
  clangASTMatchers
  clangBasic
  clangLex
  )
