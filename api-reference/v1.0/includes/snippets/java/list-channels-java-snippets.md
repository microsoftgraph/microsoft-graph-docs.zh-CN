---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dac50d937f0cd99858485af3f833cb857029f75
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968000"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelCollectionPage channels = graphClient.teams("{id}").channels()
    .buildRequest()
    .get();

```