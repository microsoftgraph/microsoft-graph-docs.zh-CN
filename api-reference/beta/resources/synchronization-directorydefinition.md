---
title: directoryDefinition 资源类型
description: 提供有关目录和其对象的同步引擎信息。 此资源告知同步引擎，例如目录有对象名为**用户**和**组**，这些对象，并为这些属性的类型支持哪些属性。 为了参与同步规则和对象映射的对象和属性，必须作为目录定义的一部分定义它们。
ms.openlocfilehash: ddc32237efc18d43da23d815aea00ee01b2650be
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049011"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="1c86b-105">directoryDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c86b-105">directoryDefinition resource type</span></span>

> <span data-ttu-id="1c86b-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c86b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c86b-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c86b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c86b-108">提供有关目录和其对象的同步引擎信息。</span><span class="sxs-lookup"><span data-stu-id="1c86b-108">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="1c86b-109">此资源告知同步引擎，例如目录有对象名为**用户**和**组**，这些对象，并为这些属性的类型支持哪些属性。</span><span class="sxs-lookup"><span data-stu-id="1c86b-109">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="1c86b-110">为了参与[同步规则](synchronization-synchronizationrule.md)和[对象映射](synchronization-objectmapping.md)的对象和属性，必须作为目录定义的一部分定义它们。</span><span class="sxs-lookup"><span data-stu-id="1c86b-110">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="1c86b-111">一般情况下，为[同步模板](synchronization-synchronizationtemplate.md)的一部分提供的默认[同步架构](synchronization-synchronizationschema.md)将定义最常用的对象和为该目录的属性。</span><span class="sxs-lookup"><span data-stu-id="1c86b-111">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="1c86b-112">但是，如果目录支持的自定义属性，您可能想要展开与您自己的自定义对象或属性的默认定义。</span><span class="sxs-lookup"><span data-stu-id="1c86b-112">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="1c86b-113">有关详细信息，请参阅[配置自定义属性同步](synchronization-configure-with-directory-extension-attributes.md)以及[与配置与目录的扩展属性](synchronization-configure-with-custom-target-attributes.md)。</span><span class="sxs-lookup"><span data-stu-id="1c86b-113">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="1c86b-114">目录定义更新[同步架构](synchronization-synchronizationschema.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="1c86b-114">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1c86b-115">属性</span><span class="sxs-lookup"><span data-stu-id="1c86b-115">Properties</span></span>

| <span data-ttu-id="1c86b-116">属性</span><span class="sxs-lookup"><span data-stu-id="1c86b-116">Property</span></span>      | <span data-ttu-id="1c86b-117">类型</span><span class="sxs-lookup"><span data-stu-id="1c86b-117">Type</span></span>      | <span data-ttu-id="1c86b-118">说明</span><span class="sxs-lookup"><span data-stu-id="1c86b-118">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="1c86b-119">id</span><span class="sxs-lookup"><span data-stu-id="1c86b-119">id</span></span>           |<span data-ttu-id="1c86b-120">字符串</span><span class="sxs-lookup"><span data-stu-id="1c86b-120">String</span></span>     |<span data-ttu-id="1c86b-121">目录标识符。</span><span class="sxs-lookup"><span data-stu-id="1c86b-121">Directory identifier.</span></span> <span data-ttu-id="1c86b-122">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1c86b-122">Not nullable.</span></span>|
|<span data-ttu-id="1c86b-123">元数据</span><span class="sxs-lookup"><span data-stu-id="1c86b-123">metadata</span></span>       |<span data-ttu-id="1c86b-124">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="1c86b-124">metadataEntry collection</span></span>    |<span data-ttu-id="1c86b-125">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1c86b-125">Additional extension properties.</span></span> <span data-ttu-id="1c86b-126">除非明确提到，不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="1c86b-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="1c86b-127">name</span><span class="sxs-lookup"><span data-stu-id="1c86b-127">name</span></span>           |<span data-ttu-id="1c86b-128">字符串</span><span class="sxs-lookup"><span data-stu-id="1c86b-128">String</span></span>     |<span data-ttu-id="1c86b-129">目录的名称。</span><span class="sxs-lookup"><span data-stu-id="1c86b-129">Name of the directory.</span></span> <span data-ttu-id="1c86b-130">必须是唯一[同步架构](synchronization-synchronizationschema.md)中。</span><span class="sxs-lookup"><span data-stu-id="1c86b-130">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="1c86b-131">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1c86b-131">Not nullable.</span></span>|
|<span data-ttu-id="1c86b-132">对象</span><span class="sxs-lookup"><span data-stu-id="1c86b-132">objects</span></span>        |<span data-ttu-id="1c86b-133">[objectDefinition](synchronization-objectdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="1c86b-133">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="1c86b-134">目录支持的对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1c86b-134">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c86b-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c86b-135">JSON representation</span></span>

<span data-ttu-id="1c86b-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c86b-136">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="1c86b-137">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="1c86b-137">JSON Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->