---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b43f6f21a1383f55a8bce45c125e244611b501f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209891"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJobCollectionPage jobs = graphClient.print().shares("{printerShareId}").jobs()
    .buildRequest()
    .get();

```