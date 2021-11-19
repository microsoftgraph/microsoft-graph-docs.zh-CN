---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0d1abf25758bcb7c3fcd4e6ba43d4f1d4f03f60
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091500"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Authentication().PhoneMethods().Get(options)


```