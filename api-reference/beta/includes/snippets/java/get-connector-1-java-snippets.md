---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c22aa8d0d23ed9f4f1035c87e4499fc15a41a8cb578024efd1a5dee6810bf243
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105649"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Connector connector = graphClient.onPremisesPublishingProfiles("applicationProxy").connectors("{id}")
    .buildRequest()
    .get();

```