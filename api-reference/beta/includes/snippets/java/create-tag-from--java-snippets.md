---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cdef22f20a2f4cacc0d4d3d7b1957c2fd18b916001a10ce97e253df837ea1d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161506"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Tag tag = new Tag();
tag.displayName = "Privileged";
tag.description = "The document is privileged";
tag.additionalDataManager().put("parent@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"));

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags()
    .buildRequest()
    .post(tag);

```