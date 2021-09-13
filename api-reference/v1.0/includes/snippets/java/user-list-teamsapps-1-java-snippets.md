---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b25f2b306b0a5bd36f59174729a00d4154f4d4c7cb3fe552adc1faaa9f36ac63
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333455"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallation userScopeTeamsAppInstallation = graphClient.users("5b649834-7412-4cce-9e69-176e95a394f5").teamwork().installedApps("NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk")
    .buildRequest()
    .get();

```