---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61b2dc6a5043828dd243ea6ebea42de4a2174735
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975919"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("forcedelete", "true"));

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags("9985bd266f2f459cbebc81522734b452")
    .buildRequest( requestOptions )
    .delete();

```