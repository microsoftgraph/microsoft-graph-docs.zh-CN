---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79839dcce645744aaae16c66ebfa27234c08e5a5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971655"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.appCatalogs().teamsApps("06805b9e-77e3-4b93-ac81-525eb87513b8")
    .buildRequest()
    .delete();

```