---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 193226c070ae115e4b0681f7c6c90163cdfdbd88
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087433"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Identity().UserFlowAttributes().Get(options)


```