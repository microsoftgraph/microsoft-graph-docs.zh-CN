---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e3d13d5e71c615a2f49d3bf1c6a6e4640ef32d2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210765"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBrandingLocalization organizationalBrandingLocalization = graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding().localizations("fr")
    .buildRequest()
    .get();

```