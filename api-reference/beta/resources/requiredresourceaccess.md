---
title: requiredResourceAccess 资源类型
description: 指定一组的 OAuth 2.0 权限范围和指定的资源的应用程序需要访问下的应用程序角色。 指定的 OAuth 2.0 权限范围可能请求 （通过**requiredResourceAccess**集合） 的客户端应用程序时调用资源应用程序。 应用程序实体的**requiredResourceAccess**属性是**ReqiredResourceAccess**的集合。
localization_priority: Normal
ms.openlocfilehash: 473126365a7f0b3ba3ab0371322ff90bd36318e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856166"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="bd152-105">requiredResourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd152-105">requiredResourceAccess resource type</span></span>

> <span data-ttu-id="bd152-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bd152-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd152-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bd152-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd152-108">指定一组的 OAuth 2.0 权限范围和指定的资源的应用程序需要访问下的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="bd152-108">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="bd152-109">指定的 OAuth 2.0 权限范围可能请求 （通过**requiredResourceAccess**集合） 的客户端应用程序时调用资源应用程序。</span><span class="sxs-lookup"><span data-stu-id="bd152-109">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="bd152-110">[应用程序](application.md)实体的**requiredResourceAccess**属性是**ReqiredResourceAccess**的集合。</span><span class="sxs-lookup"><span data-stu-id="bd152-110">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bd152-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd152-111">JSON representation</span></span>

<span data-ttu-id="bd152-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd152-112">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="bd152-113">属性</span><span class="sxs-lookup"><span data-stu-id="bd152-113">Properties</span></span>
| <span data-ttu-id="bd152-114">属性</span><span class="sxs-lookup"><span data-stu-id="bd152-114">Property</span></span>     | <span data-ttu-id="bd152-115">类型</span><span class="sxs-lookup"><span data-stu-id="bd152-115">Type</span></span>   |<span data-ttu-id="bd152-116">Description</span><span class="sxs-lookup"><span data-stu-id="bd152-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd152-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="bd152-117">resourceAccess</span></span>|<span data-ttu-id="bd152-118">[ResourceAccess](resourceaccess.md)集合</span><span class="sxs-lookup"><span data-stu-id="bd152-118">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="bd152-119">OAuth2.0 权限范围和应用程序需要从指定的资源的应用程序角色的列表。</span><span class="sxs-lookup"><span data-stu-id="bd152-119">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="bd152-120">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="bd152-120">resourceAppId</span></span>|<span data-ttu-id="bd152-121">字符串</span><span class="sxs-lookup"><span data-stu-id="bd152-121">String</span></span>|<span data-ttu-id="bd152-122">应用程序需要访问资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bd152-122">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="bd152-123">这应该是等于**appId**上的目标资源应用程序声明。</span><span class="sxs-lookup"><span data-stu-id="bd152-123">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
