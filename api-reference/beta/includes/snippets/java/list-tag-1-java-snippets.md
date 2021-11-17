---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8aeb992e9cc89f8873c835abc7373b3814df2411cc1b5a67195a8383cf3eb14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903420"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TagCollectionPage tags = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags()
    .buildRequest()
    .get();

```