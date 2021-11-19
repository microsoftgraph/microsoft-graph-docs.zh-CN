---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92be54491d91b6f4cc6ca8e7ca2f0c5c8e01d4d8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099575"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().AuthenticationFlowsPolicy().Get(options)


```