---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76714bb19f003a742616adfc372714dd3a2b8edcbc8ba26581ef7f8b17b53a7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904209"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeCard timeCard = graphClient.teams("fd15cad8-80f6-484f-9666-3caf695fbf32").schedule().timeCards("TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972")
    .buildRequest()
    .get();

```