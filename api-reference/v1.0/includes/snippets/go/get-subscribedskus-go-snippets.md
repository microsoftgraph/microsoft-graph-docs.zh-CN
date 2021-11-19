---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c13ee0a203c445ea5e4dcaf4faa4f6065735a97
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092139"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.SubscribedSkus().Get(options)


```