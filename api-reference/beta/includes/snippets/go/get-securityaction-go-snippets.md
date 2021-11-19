---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67c8e34dd2dc7047cba412522412960ab0090af3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088515"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

securityActionId := "securityAction-id"
result, err := graphClient.Security().SecurityActionsById(&securityActionId).Get(options)


```