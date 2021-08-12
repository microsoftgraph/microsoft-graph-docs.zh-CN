---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ecc018e40c056173bee17c0031a9df942e7e00becbdd5614a71af4b06bd2c01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240507"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = graphClient.me().events("AAMkADAGu0AABIGYDZAAA=")
    .buildRequest()
    .select("isOnlineMeeting,onlineMeetingProvider,onlineMeeting")
    .get();

```