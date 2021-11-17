---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0134dbc47eaf80047beab132d30440521a81c8aa5bf506b1d7704806243ed87b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333650"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var expression = "Replace([preferredLanguage], \"-\", , , \"_\", ,  )";

AttributeDefinition targetAttributeDefinition = null;

var testInputObject = new ExpressionInputObject
{
    Definition = null,
    Properties = new List<StringKeyObjectValuePair>()
    {
        new StringKeyObjectValuePair
        {
            Key = "objectId",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "66E4A8CC-1B7B-435E-95F8-F06CEA133828"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "IsSoftDeleted",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "false"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "accountEnabled",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "true"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "streetAddress",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "1 Redmond Way"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "city",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Redmond"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "state",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "WA"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "postalCode",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "98052"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "country",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "USA"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "department",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sales"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "displayName",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "John Smith"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute1",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 1"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute2",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 2"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute3",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 3"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute4",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 4"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute5",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 5"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute6",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 6"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute7",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 1"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute8",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 1"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute9",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 1"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute10",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 1"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute11",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 1"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute12",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 1"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute13",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 1"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute14",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 1"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "extensionAttribute15",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Sample 1"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "givenName",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "John"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "jobTitle",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Finance manager"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "mail",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "johns@contoso.com"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "mailNickname",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "johns"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "manager",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "maxs@contoso.com"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "mobile",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "425-555-0010"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "onPremisesSecurityIdentifier",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "66E4A8CC-1B7B-435E-95F8-F06CEA133828"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "passwordProfile.password",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", ""}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "physicalDeliveryOfficeName",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Main Office"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "preferredLanguage",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "EN-US"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "proxyAddresses",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", ""}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "surname",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "Smith"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "telephoneNumber",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "425-555-0011"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "userPrincipalName",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value", "johns@contoso.com"}
            }
        },
        new StringKeyObjectValuePair
        {
            Key = "appRoleAssignments",
            AdditionalData = new Dictionary<string, object>()
            {
                {"value@odata.type", "#Collection(String)"},
                {"value", "[\"Default Assignment\"]"}
            }
        }
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"].Schema
    .ParseExpression(expression,testInputObject,targetAttributeDefinition)
    .Request()
    .PostAsync();

```