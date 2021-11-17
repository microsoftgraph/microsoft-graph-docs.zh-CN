---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0381a2331dfbcc1710e3a3908dc013717bf218704e6613c70a6d32550430783a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163588"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.admin().windows().updates().updatableAssets("{azureADDeviceId}")
    .buildRequest()
    .delete();

```