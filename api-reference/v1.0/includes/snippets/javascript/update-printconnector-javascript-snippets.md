---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 587bd5cd368b7e1cb8a9d8b3144053edaed1d369
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776975"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printConnector = {
  displayName: 'ConnectorName',
  fullyQualifiedDomainName: 'CONNECTOR-MACHINE',
  operatingSystem: 'Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555',
  appVersion: '0.19.7338.23496',
  location: {
    latitude: 1.1,
    longitude: 2.2,
    altitudeInMeters: 3
  }
};

await client.api('/print/connectors/{printConnectorId}')
    .update(printConnector);

```