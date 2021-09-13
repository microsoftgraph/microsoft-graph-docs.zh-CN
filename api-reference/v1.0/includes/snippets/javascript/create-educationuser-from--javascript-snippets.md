---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d8236d09a16efb462182b5d6c72e5daf2ed5130c544787c70be3fd6e9dfdfbe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163276"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.type': '#microsoft.graph.educationUser',
  primaryRole: 'String',
  middleName: 'String',
  externalSource: 'String',
  externalSourceDetail: 'String',
  residenceAddress: {
    '@odata.type': 'microsoft.graph.physicalAddress'
  },
  mailingAddress: {
    '@odata.type': 'microsoft.graph.physicalAddress'
  },
  student: {
    '@odata.type': 'microsoft.graph.educationStudent'
  },
  teacher: {
    '@odata.type': 'microsoft.graph.educationTeacher'
  },
  createdBy: {
    '@odata.type': 'microsoft.graph.identitySet'
  },
  accountEnabled: 'Boolean',
  assignedLicenses: [
    {
      '@odata.type': 'microsoft.graph.assignedLicense'
    }
  ],
  assignedPlans: [
    {
      '@odata.type': 'microsoft.graph.assignedPlan'
    }
  ],
  businessPhones: [
    'String'
  ],
  department: 'String',
  displayName: 'String',
  givenName: 'String',
  mail: 'String',
  mailNickname: 'String',
  mobilePhone: 'String',
  passwordPolicies: 'String',
  passwordProfile: {
    '@odata.type': 'microsoft.graph.passwordProfile'
  },
  officeLocation: 'String',
  preferredLanguage: 'String',
  provisionedPlans: [
    {
      '@odata.type': 'microsoft.graph.provisionedPlan'
    }
  ],
  refreshTokensValidFromDateTime: 'String (timestamp)',
  showInAddressList: 'Boolean',
  surname: 'String',
  usageLocation: 'String',
  userPrincipalName: 'String',
  userType: 'String',
  onPremisesInfo: {
    '@odata.type': 'microsoft.graph.educationOnPremisesInfo'
  }
};

await client.api('/education/users')
    .post(educationUser);

```