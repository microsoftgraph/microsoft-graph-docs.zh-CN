---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42cf665a1c7d8db7a5cf01f0822c2980666a2840
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287781"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().CredentialUserRegistrationDetails().Get(nil)


```