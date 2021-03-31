---
title: windowsHelloForBusinessAuthenticationMethod 资源类型
description: 注册到用户的 Windows Hello 企业实例的表示形式。 Windows Hello 企业应用是一种登录身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cd7784bca9b6eab1390d40286431efd658c401d3
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468952"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a><span data-ttu-id="708b3-104">windowsHelloForBusinessAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="708b3-104">windowsHelloForBusinessAuthenticationMethod resource type</span></span>

<span data-ttu-id="708b3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="708b3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="708b3-106">注册到用户的 Windows Hello 企业身份验证方法的表示形式。</span><span class="sxs-lookup"><span data-stu-id="708b3-106">A representation of a Windows Hello for Business authentication method registered to a user.</span></span> <span data-ttu-id="708b3-107">Windows Hello 企业应用是 Windows 设备的登录身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="708b3-107">Windows Hello for Business is a sign-in authentication method for Windows devices.</span></span>

<span data-ttu-id="708b3-108">继承自 [authenticationMethod](../resources/authenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="708b3-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="708b3-109">方法</span><span class="sxs-lookup"><span data-stu-id="708b3-109">Methods</span></span>
|<span data-ttu-id="708b3-110">方法</span><span class="sxs-lookup"><span data-stu-id="708b3-110">Method</span></span>|<span data-ttu-id="708b3-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="708b3-111">Return type</span></span>|<span data-ttu-id="708b3-112">说明</span><span class="sxs-lookup"><span data-stu-id="708b3-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="708b3-113">列出 windowsHelloForBusinessAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="708b3-113">List windowsHelloForBusinessAuthenticationMethods</span></span>](../api/windowshelloforbusinessauthenticationmethod-list.md)|<span data-ttu-id="708b3-114">[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="708b3-114">[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) collection</span></span>|<span data-ttu-id="708b3-115">获取 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="708b3-115">Get a list of the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="708b3-116">获取 windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="708b3-116">Get windowsHelloForBusinessAuthenticationMethod</span></span>](../api/windowshelloforbusinessauthenticationmethod-get.md)|[<span data-ttu-id="708b3-117">windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="708b3-117">windowsHelloForBusinessAuthenticationMethod</span></span>](../resources/windowshelloforbusinessauthenticationmethod.md)|<span data-ttu-id="708b3-118">读取 [windowsHelloForBusinessAuthenticationMethod 对象的属性和](../resources/windowshelloforbusinessauthenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="708b3-118">Read the properties and relationships of a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="708b3-119">删除 windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="708b3-119">Delete windowsHelloForBusinessAuthenticationMethod</span></span>](../api/windowshelloforbusinessauthenticationmethod-delete.md)|<span data-ttu-id="708b3-120">无</span><span class="sxs-lookup"><span data-stu-id="708b3-120">None</span></span>|<span data-ttu-id="708b3-121">删除 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="708b3-121">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="708b3-122">属性</span><span class="sxs-lookup"><span data-stu-id="708b3-122">Properties</span></span>
|<span data-ttu-id="708b3-123">属性</span><span class="sxs-lookup"><span data-stu-id="708b3-123">Property</span></span>|<span data-ttu-id="708b3-124">类型</span><span class="sxs-lookup"><span data-stu-id="708b3-124">Type</span></span>|<span data-ttu-id="708b3-125">说明</span><span class="sxs-lookup"><span data-stu-id="708b3-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="708b3-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="708b3-126">createdDateTime</span></span>|<span data-ttu-id="708b3-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="708b3-127">DateTimeOffset</span></span>|<span data-ttu-id="708b3-128">注册此 Windows Hello 企业密钥的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="708b3-128">The date and time that this Windows Hello for Business key was registered.</span></span>|
|<span data-ttu-id="708b3-129">displayName</span><span class="sxs-lookup"><span data-stu-id="708b3-129">displayName</span></span>|<span data-ttu-id="708b3-130">String</span><span class="sxs-lookup"><span data-stu-id="708b3-130">String</span></span>|<span data-ttu-id="708b3-131">注册 Windows Hello 企业版本的设备的名称</span><span class="sxs-lookup"><span data-stu-id="708b3-131">The name of the device on which Windows Hello for Business is registered</span></span>|
|<span data-ttu-id="708b3-132">id</span><span class="sxs-lookup"><span data-stu-id="708b3-132">id</span></span>|<span data-ttu-id="708b3-133">String</span><span class="sxs-lookup"><span data-stu-id="708b3-133">String</span></span>|<span data-ttu-id="708b3-134">此身份验证方法的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="708b3-134">A unique identifier for this authentication method.</span></span> <span data-ttu-id="708b3-135">继承自 [authenticationMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="708b3-135">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="708b3-136">keyStrength</span><span class="sxs-lookup"><span data-stu-id="708b3-136">keyStrength</span></span>|<span data-ttu-id="708b3-137">authenticationMethodKeyStrength</span><span class="sxs-lookup"><span data-stu-id="708b3-137">authenticationMethodKeyStrength</span></span>|<span data-ttu-id="708b3-138">此 Windows Hello 企业密钥的关键强度。</span><span class="sxs-lookup"><span data-stu-id="708b3-138">Key strength of this Windows Hello for Business key.</span></span> <span data-ttu-id="708b3-139">可取值为：`normal`、`weak`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="708b3-139">Possible values are: `normal`, `weak`, `unknown`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="708b3-140">关系</span><span class="sxs-lookup"><span data-stu-id="708b3-140">Relationships</span></span>
|<span data-ttu-id="708b3-141">关系</span><span class="sxs-lookup"><span data-stu-id="708b3-141">Relationship</span></span>|<span data-ttu-id="708b3-142">类型</span><span class="sxs-lookup"><span data-stu-id="708b3-142">Type</span></span>|<span data-ttu-id="708b3-143">说明</span><span class="sxs-lookup"><span data-stu-id="708b3-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="708b3-144">设备</span><span class="sxs-lookup"><span data-stu-id="708b3-144">device</span></span>|[<span data-ttu-id="708b3-145">设备</span><span class="sxs-lookup"><span data-stu-id="708b3-145">device</span></span>](../resources/device.md)|<span data-ttu-id="708b3-146">此 Windows Hello 企业密钥所在的已注册设备。</span><span class="sxs-lookup"><span data-stu-id="708b3-146">The registered device on which this Windows Hello for Business key resides.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="708b3-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="708b3-147">JSON representation</span></span>
<span data-ttu-id="708b3-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="708b3-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "createdDateTime": "String",
  "keyStrength": {"@odata.type": "microsoft.graph.authenticationMethodKeyStrength"}
}
```
