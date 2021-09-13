---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 324216f3d323cdff336277569bdbaceb4cd3d716b0fef9615873e679147929ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279679"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directoryObjects("{id}")
    .buildRequest()
    .get();

```