---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d10a6c7984b085dbc033f48d8699cc65cd11f4c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102605"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().CredentialUserRegistrationDetails().Get(options)


```