---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bbe3da32617ea794c6aa90925268a630d466606
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508921"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "2441b489-4f12-4882-b039-8f6006bd66da";

graphClient.policies().featureRolloutPolicies("{id}").appliesTo().references()
    .buildRequest()
    .post(directoryObject);

```