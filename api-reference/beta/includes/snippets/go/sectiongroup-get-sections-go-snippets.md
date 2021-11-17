---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28bbca4f41864a033e880c4d40b395b90af660ec
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979898"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

sectionGroupId := "sectionGroup-id"
result, err := graphClient.Me().Onenote().SectionGroupsById(&sectionGroupId).Sections().Get(options)


```