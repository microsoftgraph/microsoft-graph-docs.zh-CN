---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95c5fdbb25d43a13ab4869954ce0fd7259995a43ebe01a426bd60867c38f38c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328693"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallationCollectionPage installedApps = graphClient.users("{id}").teamwork().installedApps()
    .buildRequest()
    .get();

```