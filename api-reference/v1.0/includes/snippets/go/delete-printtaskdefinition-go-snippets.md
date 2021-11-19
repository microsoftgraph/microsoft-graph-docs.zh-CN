---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a650d6edd575f49cd7afb88d965ec18729056420
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086496"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printTaskDefinitionId := "printTaskDefinition-id"
graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).Delete(options)


```