---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbcaca18dcd87ab745480d312dd4ab148b14e255
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326874"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().GetCredentialUserRegistrationCount()().Get()


```