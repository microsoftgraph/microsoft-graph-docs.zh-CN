---
title: requiredResourceAccess 资源类型
description: 指定应用程序需要访问的指定资源下的 OAuth 2.0 权限范围和应用角色的集合。 调用资源应用程序时, 客户端应用程序可能会请求指定的 OAuth 2.0 权限范围 (通过**requiredResourceAccess**集合)。 Application 实体的**requiredResourceAccess**属性是**ReqiredResourceAccess**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6c7fec2027e5e987c66f868cc4a69555141bdbf9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965416"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="5520c-105">requiredResourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="5520c-105">requiredResourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5520c-106">指定应用程序需要访问的指定资源下的 OAuth 2.0 权限范围和应用角色的集合。</span><span class="sxs-lookup"><span data-stu-id="5520c-106">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="5520c-107">调用资源应用程序时, 客户端应用程序可能会请求指定的 OAuth 2.0 权限范围 (通过**requiredResourceAccess**集合)。</span><span class="sxs-lookup"><span data-stu-id="5520c-107">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="5520c-108">[Application](application.md)实体的**RequiredResourceAccess**属性是**ReqiredResourceAccess**的集合。</span><span class="sxs-lookup"><span data-stu-id="5520c-108">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="5520c-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5520c-109">JSON representation</span></span>

<span data-ttu-id="5520c-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5520c-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a><span data-ttu-id="5520c-111">属性</span><span class="sxs-lookup"><span data-stu-id="5520c-111">Properties</span></span>
| <span data-ttu-id="5520c-112">属性</span><span class="sxs-lookup"><span data-stu-id="5520c-112">Property</span></span>     | <span data-ttu-id="5520c-113">类型</span><span class="sxs-lookup"><span data-stu-id="5520c-113">Type</span></span>   |<span data-ttu-id="5520c-114">说明</span><span class="sxs-lookup"><span data-stu-id="5520c-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5520c-115">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="5520c-115">resourceAccess</span></span>|<span data-ttu-id="5520c-116">[ResourceAccess](resourceaccess.md)集合</span><span class="sxs-lookup"><span data-stu-id="5520c-116">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="5520c-117">应用程序需要指定资源中的 OAuth 2.0 权限范围和应用程序角色的列表。</span><span class="sxs-lookup"><span data-stu-id="5520c-117">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="5520c-118">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="5520c-118">resourceAppId</span></span>|<span data-ttu-id="5520c-119">String</span><span class="sxs-lookup"><span data-stu-id="5520c-119">String</span></span>|<span data-ttu-id="5520c-120">应用程序需要访问的资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5520c-120">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="5520c-121">此值应等于在目标资源应用程序上声明的**appId** 。</span><span class="sxs-lookup"><span data-stu-id="5520c-121">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
