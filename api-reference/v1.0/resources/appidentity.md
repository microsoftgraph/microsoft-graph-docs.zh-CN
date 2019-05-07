---
title: appIdentity 资源类型
description: 指示执行了操作或已更改的应用程序的标识。 包括应用程序 Id、名称、服务主体 ID 和名称。 此资源由 directoryAudit API 调用
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a4e7f5a21d5140537e745f7234186ad3b24098f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629353"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="bb14f-105">appIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb14f-105">appIdentity resource type</span></span>

<span data-ttu-id="bb14f-106">指示执行了操作或已更改的应用程序的标识。</span><span class="sxs-lookup"><span data-stu-id="bb14f-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="bb14f-107">包括应用程序 ID、名称和服务主体 ID 和名称。</span><span class="sxs-lookup"><span data-stu-id="bb14f-107">Includes application ID, name, and service principal ID and name.</span></span> <span data-ttu-id="bb14f-108">[Get directoryAudit](../api/directoryaudit-get.md)操作使用此资源。</span><span class="sxs-lookup"><span data-stu-id="bb14f-108">This resource is used by the [Get directoryAudit](../api/directoryaudit-get.md) operation.</span></span>

## <a name="properties"></a><span data-ttu-id="bb14f-109">属性</span><span class="sxs-lookup"><span data-stu-id="bb14f-109">Properties</span></span>

| <span data-ttu-id="bb14f-110">属性</span><span class="sxs-lookup"><span data-stu-id="bb14f-110">Property</span></span>     | <span data-ttu-id="bb14f-111">类型</span><span class="sxs-lookup"><span data-stu-id="bb14f-111">Type</span></span>   |<span data-ttu-id="bb14f-112">说明</span><span class="sxs-lookup"><span data-stu-id="bb14f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb14f-113">appId</span><span class="sxs-lookup"><span data-stu-id="bb14f-113">appId</span></span>|<span data-ttu-id="bb14f-114">String</span><span class="sxs-lookup"><span data-stu-id="bb14f-114">String</span></span>|<span data-ttu-id="bb14f-115">表示唯一 GUID（表示 Azure Active Directory 中的应用程序 ID）。</span><span class="sxs-lookup"><span data-stu-id="bb14f-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="bb14f-116">displayName</span><span class="sxs-lookup"><span data-stu-id="bb14f-116">displayName</span></span>|<span data-ttu-id="bb14f-117">字符串</span><span class="sxs-lookup"><span data-stu-id="bb14f-117">String</span></span>|<span data-ttu-id="bb14f-118">引用 Azure 门户中显示的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="bb14f-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="bb14f-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="bb14f-119">servicePrincipalId</span></span>|<span data-ttu-id="bb14f-120">字符串</span><span class="sxs-lookup"><span data-stu-id="bb14f-120">String</span></span>|<span data-ttu-id="bb14f-121">指在 Azure Active Directory 中指示对应应用程序的服务主体 Id 的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="bb14f-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="bb14f-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb14f-122">servicePrincipalName</span></span>|<span data-ttu-id="bb14f-123">String</span><span class="sxs-lookup"><span data-stu-id="bb14f-123">String</span></span>|<span data-ttu-id="bb14f-124">引用服务主体名称是租户中的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="bb14f-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bb14f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb14f-125">JSON representation</span></span>

<span data-ttu-id="bb14f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb14f-126">Here is a JSON representation of the resource.</span></span>

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
