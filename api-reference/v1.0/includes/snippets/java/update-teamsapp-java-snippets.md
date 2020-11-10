---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83deb5c62835237b575dd342798996db71c98933
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964248"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] teamsApp = Base64.getDecoder().decode("[Zip file containing a Teams app package]");
    graphClient.appCatalogs().teamsApps("06805b9e-77e3-4b93-ac81-525eb87513b8")
    .buildRequest()
    .put(teamsApp);

```