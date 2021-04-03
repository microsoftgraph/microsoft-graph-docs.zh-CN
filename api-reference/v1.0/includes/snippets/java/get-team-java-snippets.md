---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d5c3c27b8aeadbfd5c55447bb6752f3665f275c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507884"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = graphClient.teams("893075dd-2487-4122-925f-022c42e20265")
    .buildRequest()
    .get();

```