---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea48185f9b72ffc53f3378694063b7bc6d4c3bd3fc434a94a228d29d55852c5e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278658"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.appCatalogs().teamsApps("06805b9e-77e3-4b93-ac81-525eb87513b8")
    .buildRequest()
    .delete();

```