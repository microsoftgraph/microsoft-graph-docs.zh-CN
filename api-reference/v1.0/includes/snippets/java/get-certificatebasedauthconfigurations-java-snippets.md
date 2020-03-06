---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27e6797c0e757fd91ed1218894e4e65c25740490
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638682"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICertificateBasedAuthConfigurationCollectionPage certificateBasedAuthConfiguration = graphClient.organization("{id}").certificateBasedAuthConfiguration()
    .buildRequest()
    .get();

```