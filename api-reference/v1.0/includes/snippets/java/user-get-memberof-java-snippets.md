---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01a3cdb05b62bba9a44e34790931b7dc24468e39
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905840"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage memberOf = graphClient.users("{id}").memberOf()
    .buildRequest()
    .get();

```