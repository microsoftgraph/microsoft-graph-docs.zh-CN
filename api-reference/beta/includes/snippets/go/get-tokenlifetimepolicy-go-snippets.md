---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7d22001f8118d5b934a1b256225a829d3760ebe
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087800"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tokenLifetimePolicyId := "tokenLifetimePolicy-id"
result, err := graphClient.Policies().TokenLifetimePoliciesById(&tokenLifetimePolicyId).Get(options)


```