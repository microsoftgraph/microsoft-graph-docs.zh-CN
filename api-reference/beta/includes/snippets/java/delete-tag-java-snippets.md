---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a525d777f329d8d69b174e455f9a92c0577a2785702f374fcdfaaa9ca8b29569
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332513"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("forcedelete", "true"));

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags("9985bd266f2f459cbebc81522734b452")
    .buildRequest( requestOptions )
    .delete();

```