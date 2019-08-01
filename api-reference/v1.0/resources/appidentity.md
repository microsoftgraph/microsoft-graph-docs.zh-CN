---
title: appIdentity 资源类型
description: 指示执行了操作或已更改的应用程序的标识。 包括应用程序 Id、名称、服务主体 ID 和名称。 此资源由 directoryAudit API 调用
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a8b2c9185f595bf4ab534dda5a73b1a5f40fd17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030091"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="f9ffa-105">appIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9ffa-105">appIdentity resource type</span></span>

<span data-ttu-id="f9ffa-106">指示执行了操作或已更改的应用程序的标识。</span><span class="sxs-lookup"><span data-stu-id="f9ffa-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="f9ffa-107">包括应用程序 ID、名称和服务主体 ID 和名称。</span><span class="sxs-lookup"><span data-stu-id="f9ffa-107">Includes application ID, name, and service principal ID and name.</span></span> <span data-ttu-id="f9ffa-108">[Get directoryAudit](../api/directoryaudit-get.md)操作使用此资源。</span><span class="sxs-lookup"><span data-stu-id="f9ffa-108">This resource is used by the [Get directoryAudit](../api/directoryaudit-get.md) operation.</span></span>

## <a name="properties"></a><span data-ttu-id="f9ffa-109">属性</span><span class="sxs-lookup"><span data-stu-id="f9ffa-109">Properties</span></span>

| <span data-ttu-id="f9ffa-110">属性</span><span class="sxs-lookup"><span data-stu-id="f9ffa-110">Property</span></span>     | <span data-ttu-id="f9ffa-111">类型</span><span class="sxs-lookup"><span data-stu-id="f9ffa-111">Type</span></span>   |<span data-ttu-id="f9ffa-112">说明</span><span class="sxs-lookup"><span data-stu-id="f9ffa-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9ffa-113">appId</span><span class="sxs-lookup"><span data-stu-id="f9ffa-113">appId</span></span>|<span data-ttu-id="f9ffa-114">String</span><span class="sxs-lookup"><span data-stu-id="f9ffa-114">String</span></span>|<span data-ttu-id="f9ffa-115">表示唯一 GUID（表示 Azure Active Directory 中的应用程序 ID）。</span><span class="sxs-lookup"><span data-stu-id="f9ffa-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="f9ffa-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f9ffa-116">displayName</span></span>|<span data-ttu-id="f9ffa-117">字符串</span><span class="sxs-lookup"><span data-stu-id="f9ffa-117">String</span></span>|<span data-ttu-id="f9ffa-118">引用 Azure 门户中显示的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="f9ffa-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="f9ffa-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="f9ffa-119">servicePrincipalId</span></span>|<span data-ttu-id="f9ffa-120">String</span><span class="sxs-lookup"><span data-stu-id="f9ffa-120">String</span></span>|<span data-ttu-id="f9ffa-121">指在 Azure Active Directory 中指示对应应用程序的服务主体 Id 的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="f9ffa-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="f9ffa-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f9ffa-122">servicePrincipalName</span></span>|<span data-ttu-id="f9ffa-123">String</span><span class="sxs-lookup"><span data-stu-id="f9ffa-123">String</span></span>|<span data-ttu-id="f9ffa-124">引用服务主体名称是租户中的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="f9ffa-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f9ffa-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9ffa-125">JSON representation</span></span>

<span data-ttu-id="f9ffa-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9ffa-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
