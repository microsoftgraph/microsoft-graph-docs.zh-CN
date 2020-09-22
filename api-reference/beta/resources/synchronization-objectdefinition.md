---
title: objectDefinition 资源类型
description: 描述对象及其属性。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0048d11a8241e8a81bf223f337493e37aebaceda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016014"
---
# <a name="objectdefinition-resource-type"></a><span data-ttu-id="abad0-103">objectDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="abad0-103">objectDefinition resource type</span></span>

<span data-ttu-id="abad0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abad0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abad0-105">描述对象及其属性。</span><span class="sxs-lookup"><span data-stu-id="abad0-105">Describes an object and its attributes.</span></span> <span data-ttu-id="abad0-106">对象定义是 [directoryDefinition](synchronization-directorydefinition.md)的一部分，它作为 [synchronizationSchema](synchronization-synchronizationschema.md)的一部分进行更新。</span><span class="sxs-lookup"><span data-stu-id="abad0-106">Object definitions are part of [directoryDefinition](synchronization-directorydefinition.md), which is updated as part of [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="abad0-107">属性</span><span class="sxs-lookup"><span data-stu-id="abad0-107">Properties</span></span>

| <span data-ttu-id="abad0-108">属性</span><span class="sxs-lookup"><span data-stu-id="abad0-108">Property</span></span>      | <span data-ttu-id="abad0-109">类型</span><span class="sxs-lookup"><span data-stu-id="abad0-109">Type</span></span>      | <span data-ttu-id="abad0-110">说明</span><span class="sxs-lookup"><span data-stu-id="abad0-110">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="abad0-111">attributes</span><span class="sxs-lookup"><span data-stu-id="abad0-111">attributes</span></span>     |<span data-ttu-id="abad0-112">[attributeDefinition](synchronization-attributedefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="abad0-112">[attributeDefinition](synchronization-attributedefinition.md) collection</span></span>    | <span data-ttu-id="abad0-113">定义对象的属性。</span><span class="sxs-lookup"><span data-stu-id="abad0-113">Defines attributes of the object.</span></span> |
|<span data-ttu-id="abad0-114">metadata</span><span class="sxs-lookup"><span data-stu-id="abad0-114">metadata</span></span>       |<span data-ttu-id="abad0-115">[metadataEntry](synchronization-metadataentry.md) 集合</span><span class="sxs-lookup"><span data-stu-id="abad0-115">[metadataEntry](synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="abad0-116">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="abad0-116">Additional extension properties.</span></span> <span data-ttu-id="abad0-117">除非明确提到，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="abad0-117">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="abad0-118">name</span><span class="sxs-lookup"><span data-stu-id="abad0-118">name</span></span>           |<span data-ttu-id="abad0-119">String</span><span class="sxs-lookup"><span data-stu-id="abad0-119">String</span></span>     |<span data-ttu-id="abad0-120">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="abad0-120">Name of the object.</span></span> <span data-ttu-id="abad0-121">在目录定义中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="abad0-121">Must be unique within a directory definition.</span></span> <span data-ttu-id="abad0-122">不可为空。</span><span class="sxs-lookup"><span data-stu-id="abad0-122">Not nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="abad0-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="abad0-123">JSON representation</span></span>

<span data-ttu-id="abad0-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abad0-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectDefinition"
}-->

```json
{
  "attributes": [{"@odata.type": "microsoft.graph.attributeDefinition"}],
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "name": "String"
}
```

## <a name="json-example"></a><span data-ttu-id="abad0-125">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="abad0-125">JSON Example</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectDefinition"
}-->

```json
{
    "attributes": [
        {
            "anchor": true,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "objectId",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "IsSoftDeleted",
            "required": true,
            "referencedObjects": [],
            "type": "Boolean"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "accountEnabled",
            "required": true,
            "referencedObjects": [],
            "type": "Boolean"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "streetAddress",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "city",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "state",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "postalCode",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "country",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "companyName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "department",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "dirSyncEnabled",
            "required": false,
            "referencedObjects": [],
            "type": "Boolean"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "displayName",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "extensionAttribute1",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "facsimileTelephoneNumber",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "givenName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "jobTitle",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "mail",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "mailNickname",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "manager",
            "required": false,
            "referencedObjects": [
                {
                    "referencedObjectName": "User",
                    "referencedProperty": null
                }
            ],
            "type": "Reference"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "mobile",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "onPremisesSecurityIdentifier",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "originalUserPrincipalName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "passwordProfile.password",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "physicalDeliveryOfficeName",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "preferredLanguage",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": true,
            "mutability": "ReadWrite",
            "name": "proxyAddresses",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "surname",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "telephoneNumber",
            "required": false,
            "referencedObjects": [],
            "type": "String"
        },
        {
            "anchor": false,
            "caseExact": false,
            "defaultValue": null,
            "metadata": [],
            "multivalued": false,
            "mutability": "ReadWrite",
            "name": "userPrincipalName",
            "required": true,
            "referencedObjects": [],
            "type": "String"
        }
    ],
    "metadata": [
        {
            "key": "IsSoftDeletionSupported",
            "value": "true"
        },
        {
            "key": "ConnectorDataStorageRequired",
            "value": "true"
        },
        {
            "key": "IsSynchronizeAllSupported",
            "value": "true"
        },
        {
            "key": "PropertyNameAccountEnabled",
            "value": "accountEnabled"
        },
        {
            "key": "PropertyNameSoftDeleted",
            "value": "IsSoftDeleted"
        }
    ],
    "name": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


