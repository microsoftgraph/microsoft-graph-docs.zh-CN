---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc5288e66d2868d12fb041ff7ef9b206a710517f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099235"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Teamwork().WorkforceIntegrations().Get(options)


```