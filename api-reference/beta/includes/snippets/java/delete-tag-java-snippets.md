---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2eb9265d080170e1fd27025aa82cdb89872607e3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776429"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("forcedelete", "true"));

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags("9985bd266f2f459cbebc81522734b452")
    .buildRequest( requestOptions )
    .delete();

```