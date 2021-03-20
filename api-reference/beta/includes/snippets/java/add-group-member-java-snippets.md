---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4425c46e6f33adc7211e6e2e26a036767d106251
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971307"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.groups("{group-id}").members().references()
    .buildRequest()
    .post(directoryObject);

```