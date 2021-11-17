---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cea73180b4fbf0f70523d0f4e53f6a979b36fe02d81a3452ba0b19a8d1304e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162710"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("871dbd5c-3a6a-4392-bfe1-042452793a50").schedule().timeCards("3895809b-a618-4c0d-86a0-d42b25b7d74f")
    .buildRequest()
    .delete();

```