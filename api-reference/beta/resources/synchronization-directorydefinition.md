---
title: directoryDefinition 资源类型
description: 提供有关目录及其对象的同步引擎信息。 此资源将告知同步引擎, 例如, 目录包含名为**user**和**group**的对象、支持这些对象的属性以及这些属性的类型。 为了使对象和属性参与同步规则和对象映射, 必须将它们定义为目录定义的一部分。
localization_priority: Normal
ms.openlocfilehash: 22ba4a7f3b5b5d3154ec6b3f5d42bd6f1b8f09d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582059"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="bdd01-105">directoryDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdd01-105">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdd01-106">提供有关目录及其对象的同步引擎信息。</span><span class="sxs-lookup"><span data-stu-id="bdd01-106">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="bdd01-107">此资源将告知同步引擎, 例如, 目录包含名为**user**和**group**的对象、支持这些对象的属性以及这些属性的类型。</span><span class="sxs-lookup"><span data-stu-id="bdd01-107">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="bdd01-108">为了使对象和属性参与[同步规则](synchronization-synchronizationrule.md)和[对象映射](synchronization-objectmapping.md), 必须将它们定义为目录定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="bdd01-108">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="bdd01-109">通常, 作为[同步模板](synchronization-synchronizationtemplate.md)的一部分提供的默认[同步架构](synchronization-synchronizationschema.md)将为该目录定义最常用的对象和属性。</span><span class="sxs-lookup"><span data-stu-id="bdd01-109">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="bdd01-110">但是, 如果目录支持添加自定义属性, 则可能需要使用自己的自定义对象或属性扩展默认定义。</span><span class="sxs-lookup"><span data-stu-id="bdd01-110">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="bdd01-111">有关详细信息, 请参阅[配置与自定义属性的同步](synchronization-configure-with-custom-target-attributes.md)和[配置与目录扩展属性的同步](synchronization-configure-with-directory-extension-attributes.md)。</span><span class="sxs-lookup"><span data-stu-id="bdd01-111">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="bdd01-112">目录定义作为[同步架构](synchronization-synchronizationschema.md)的一部分进行更新。</span><span class="sxs-lookup"><span data-stu-id="bdd01-112">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bdd01-113">属性</span><span class="sxs-lookup"><span data-stu-id="bdd01-113">Properties</span></span>

| <span data-ttu-id="bdd01-114">属性</span><span class="sxs-lookup"><span data-stu-id="bdd01-114">Property</span></span>      | <span data-ttu-id="bdd01-115">类型</span><span class="sxs-lookup"><span data-stu-id="bdd01-115">Type</span></span>      | <span data-ttu-id="bdd01-116">说明</span><span class="sxs-lookup"><span data-stu-id="bdd01-116">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="bdd01-117">id</span><span class="sxs-lookup"><span data-stu-id="bdd01-117">id</span></span>           |<span data-ttu-id="bdd01-118">字符串</span><span class="sxs-lookup"><span data-stu-id="bdd01-118">String</span></span>     |<span data-ttu-id="bdd01-119">目录标识符。</span><span class="sxs-lookup"><span data-stu-id="bdd01-119">Directory identifier.</span></span> <span data-ttu-id="bdd01-120">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="bdd01-120">Not nullable.</span></span>|
|<span data-ttu-id="bdd01-121">metadata</span><span class="sxs-lookup"><span data-stu-id="bdd01-121">metadata</span></span>       |<span data-ttu-id="bdd01-122">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="bdd01-122">metadataEntry collection</span></span>    |<span data-ttu-id="bdd01-123">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="bdd01-123">Additional extension properties.</span></span> <span data-ttu-id="bdd01-124">除非明确提到, 否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="bdd01-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="bdd01-125">name</span><span class="sxs-lookup"><span data-stu-id="bdd01-125">name</span></span>           |<span data-ttu-id="bdd01-126">String</span><span class="sxs-lookup"><span data-stu-id="bdd01-126">String</span></span>     |<span data-ttu-id="bdd01-127">目录的名称。</span><span class="sxs-lookup"><span data-stu-id="bdd01-127">Name of the directory.</span></span> <span data-ttu-id="bdd01-128">在[同步架构](synchronization-synchronizationschema.md)中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="bdd01-128">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="bdd01-129">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="bdd01-129">Not nullable.</span></span>|
|<span data-ttu-id="bdd01-130">对象</span><span class="sxs-lookup"><span data-stu-id="bdd01-130">objects</span></span>        |<span data-ttu-id="bdd01-131">[objectDefinition](synchronization-objectdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="bdd01-131">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="bdd01-132">目录支持的对象集合。</span><span class="sxs-lookup"><span data-stu-id="bdd01-132">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdd01-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdd01-133">JSON representation</span></span>

<span data-ttu-id="bdd01-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdd01-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "id": "String",
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}]
}

```

## <a name="json-example"></a><span data-ttu-id="bdd01-135">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="bdd01-135">JSON Example</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
    "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
    "name": "salesforce.com",
    "objects": [
        {
            "attributes": [
                {
                    "anchor": true,
                    "name": "Id",
                    "type": "String"
                },
                {
                    "name": "IsActive",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "mutability": "ReadWrite",
                    "name": "Alias",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "CompanyName",
                    "type": "String"
                },
                {
                    "name": "CommunityNickname",
                    "type": "String"
                },
                {
                    "name": "Email",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "EmailEncodingKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LanguageLocaleKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "FirstName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LastName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LocaleSidKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "metadata": [
                        {
                            "key": "LinkTypeName",
                            "value": "PermissionSetAssignment"
                        },
                        {
                            "key": "LinkPropertyNames",
                            "value": "[\"PermissionSetId\"]"
                        }
                    ],
                    "name": "PermissionSets",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "PermissionSet"
                        }
                    ],
                    "type": "Reference"
                },
                {
                    "name": "ProfileId",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "ProfileName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "TimeZoneSidKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "Username",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "UserPermissionsCallCenterAutoLogin",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "name": "UserPermissionsMarketingUser",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "name": "Street",
                    "type": "String"
                },
                {
                    "name": "City",
                    "type": "String"
                },
                {
                    "name": "Division",
                    "type": "String"
                },
                {
                    "name": "EmployeeNumber",
                    "type": "String"
                },
                {
                    "name": "State",
                    "type": "String"
                },
                {
                    "name": "PostalCode",
                    "type": "String"
                },
                {
                    "name": "Country",
                    "type": "String"
                },
                {
                    "name": "Department",
                    "type": "String"
                },
                {
                    "name": "MobilePhone",
                    "type": "String"
                },
                {
                    "name": "Phone",
                    "type": "String"
                },
                {
                    "name": "Title",
                    "type": "String"
                },
                {
                    "name": "FederationIdentifier",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "ManagerId",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "User"
                        }
                    ],
                    "type": "Reference"
                },
                {
                    "name": "UserRoleId",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "UserRole"
                        }
                    ],
                    "type": "Reference"
                }
            ],
            "metadata": [
                {
                    "key": "IsSoftDeletionSupported",
                    "value": "false"
                },
                {
                    "key": "ConnectorDataStorageRequired",
                    "value": "false"
                },
                {
                    "key": "IsSynchronizeAllSupported",
                    "value": "false"
                }
            ],
            "name": "User"
        }
    ],
    "metadata": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-directorydefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
