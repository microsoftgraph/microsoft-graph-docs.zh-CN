---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a29ebb80d86517a49ef8e1353f8fab2d933048b2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086225"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contractId := "contract-id"
result, err := graphClient.ContractsById(&contractId).Get(options)


```