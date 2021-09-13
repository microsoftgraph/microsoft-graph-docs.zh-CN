---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec4257740e926c9d853ca9c2531f2d9b89fb34c892552277ef5fdc471790afaf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163527"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").installedApps("MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=")
    .buildRequest()
    .get();

```