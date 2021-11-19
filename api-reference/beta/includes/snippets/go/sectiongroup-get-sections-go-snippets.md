---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 953875671d98164879f273eda1e9ba8c39c96c09
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095150"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

sectionGroupId := "sectionGroup-id"
result, err := graphClient.Me().Onenote().SectionGroupsById(&sectionGroupId).Sections().Get(options)


```