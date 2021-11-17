---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1edf969216755cbca4d3f6e42f874ef6157e4287
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033074"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

notebookId := "notebook-id"
result, err := graphClient.Me().Onenote().NotebooksById(&notebookId).SectionGroups().Get(options)


```