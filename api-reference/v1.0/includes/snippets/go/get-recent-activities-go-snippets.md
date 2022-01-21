---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bde9e8f94e5401f35e2cc86ea1fbe86cff9ffcc8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137757"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Activities().Recent()().Get(nil)


```