---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbb3506d408542ea57166f2e547f203d62f47ca4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032964"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

presenceId := "presence-id"
result, err := graphClient.Communications().PresencesById(&presenceId).Get(options)


```