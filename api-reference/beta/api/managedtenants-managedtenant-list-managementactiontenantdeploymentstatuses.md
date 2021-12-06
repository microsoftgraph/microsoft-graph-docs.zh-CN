---
title: List managementActionTenantDeploymentStatus
description: 获取 managementActionTenantDeploymentStatus 对象及其属性的列表。
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a9681e5d6a5bc5537854971bd1e579e7bc8a6871
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981103"
---
# <a name="list-managementactiontenantdeploymentstatus"></a>List managementActionTenantDeploymentStatus
命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ManagedTenants.Read.All、ManagedTenants.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_managementactiontenantdeploymentstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-managementactiontenantdeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-managementactiontenantdeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-managementactiontenantdeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-managementactiontenantdeploymentstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-managementactiontenantdeploymentstatus-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementActionTenantDeploymentStatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses",
    "value": [
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_34298981-4fc8-4974-9486-c8909ed1521b",
            "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
            "statuses": [
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                            "status": "completed",
                            "deployedPolicyId": "949e8893-68fb-4c9d-b8a0-13c229a7e397",
                            "lastDeploymentDateTime": "2021-06-22T04:09:20.3054223Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                            "status": "completed",
                            "deployedPolicyId": "19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
                            "lastDeploymentDateTime": "2021-06-22T17:01:44.851214Z",
                            "error": null
                        }
                    ]
                }
            ]
        },
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_38227791-a88b-4fcc-81c5-58cf77668320",
            "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
            "statuses": [
                {
                    "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                    "managementActionId": "eac82706-9f32-4274-ba5b-cf1f8ecf042b",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "7fff5ebb-10bd-4493-b0bb-2d0cf6172f16",
                            "status": "completed",
                            "deployedPolicyId": "062107b4-236d-465a-ae62-3bb4bd31f276",
                            "lastDeploymentDateTime": "2021-06-17T13:19:47.3003079Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
                    "managementActionId": "55f8da1a-4eec-4fb2-9c58-4c4b3cdf7222",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "4a1c5d34-c2f7-4fd5-a7b5-4bedd95bb8f9",
                            "status": "completed",
                            "deployedPolicyId": "606cf367-2075-40c4-a587-7914b6d83dc7",
                            "lastDeploymentDateTime": "2021-06-17T15:21:17.5296126Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                            "status": "completed",
                            "deployedPolicyId": "60148b3e-39a2-4c0c-95a6-375a939aa756",
                            "lastDeploymentDateTime": "2021-06-22T05:54:42.7087204Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
                    "status": "riskAccepted",
                    "workloadActionDeploymentStatuses": []
                },
                {
                    "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
                    "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6",
                    "status": "toAddress",
                    "workloadActionDeploymentStatuses": []
                }
            ]
        },
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_4d262a25-c70a-430b-9e8e-46c31dec116b",
            "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b",
            "statuses": [
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                            "status": "completed",
                            "deployedPolicyId": "aee50adb-9445-44a8-baaf-7d16b388d708",
                            "lastDeploymentDateTime": "2021-06-18T20:21:00.0934112Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                    "managementActionId": "eac82706-9f32-4274-ba5b-cf1f8ecf042b",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "7fff5ebb-10bd-4493-b0bb-2d0cf6172f16",
                            "status": "completed",
                            "deployedPolicyId": "67635cbb-6519-44dd-bf7f-fd8752d1339b",
                            "lastDeploymentDateTime": "2021-07-09T18:53:07.113328Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                            "status": "completed",
                            "deployedPolicyId": "f296e4d5-7b4a-4c7b-977f-cd4e5bbbc0ea",
                            "lastDeploymentDateTime": "2021-07-09T20:12:33.6197104Z",
                            "error": null
                        }
                    ]
                }
            ]
        },
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_791fae7d-ffda-4187-ba69-14ed55bdb026",
            "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "tenantId": "791fae7d-ffda-4187-ba69-14ed55bdb026",
            "statuses": [
                {
                    "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                    "managementActionId": "eac82706-9f32-4274-ba5b-cf1f8ecf042b",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "7fff5ebb-10bd-4493-b0bb-2d0cf6172f16",
                            "status": "completed",
                            "deployedPolicyId": "2e628607-5908-4dea-89c3-61438dd77805",
                            "lastDeploymentDateTime": "2021-06-17T05:14:12.671197Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                            "status": "completed",
                            "deployedPolicyId": "deebefee-f378-4d2e-ab1a-a7f2bf1a010e",
                            "lastDeploymentDateTime": "2021-06-17T05:15:08.801992Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
                    "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "6a3ad0bc-5d7e-4a49-a105-c559aa4633e1",
                            "status": "completed",
                            "deployedPolicyId": "e14428f4-9890-4f6b-8416-ec40d9a59646",
                            "lastDeploymentDateTime": "2021-06-17T05:15:57.5564366Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
                    "managementActionId": "55f8da1a-4eec-4fb2-9c58-4c4b3cdf7222",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "4a1c5d34-c2f7-4fd5-a7b5-4bedd95bb8f9",
                            "status": "completed",
                            "deployedPolicyId": "220bbe5d-2167-4ba1-8c7d-67bd56b0e068",
                            "lastDeploymentDateTime": "2021-06-17T05:16:35.1968434Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                            "status": "completed",
                            "deployedPolicyId": "50553bd7-560e-4c0e-9c80-78f4ae9560e5",
                            "lastDeploymentDateTime": "2021-06-17T05:17:46.2079328Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
                    "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "46b80b42-06c7-45b4-b6fb-aa0aecace87b",
                            "status": "completed",
                            "deployedPolicyId": null,
                            "lastDeploymentDateTime": "2021-06-17T05:18:16.7581968Z",
                            "error": null
                        }
                    ]
                }
            ]
        }
    ]
}
```
