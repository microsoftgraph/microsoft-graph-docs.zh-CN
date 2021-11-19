---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79a76607ad4435ceae530a7b49ba3b4915a96024
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097164"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Profile().Patents().Get(options)


```