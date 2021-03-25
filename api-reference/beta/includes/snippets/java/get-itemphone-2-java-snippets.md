---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16b954544b0c12f9092ae2c946ed21a981c653fa
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209113"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPhoneCollectionPage phones = graphClient.me().profile().phones()
    .buildRequest()
    .get();

```