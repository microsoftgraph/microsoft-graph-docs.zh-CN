---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2849d442499d953a22ea01cabb4be057acbf3fee
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975629"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPcUserSettingId := "cloudPcUserSetting-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById(&cloudPcUserSettingId).Get(options)


```