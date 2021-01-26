---
title: windowsHelloForBusinessAuthenticationMethod 资源类型
description: 注册到用户的 Windows Hello 企业实例的表示形式。 Windows Hello 企业应用是一种登录身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dcbbebf03a91563e5504eb3032f57f973a4c3ede
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982479"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a><span data-ttu-id="3ff86-104">windowsHelloForBusinessAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ff86-104">windowsHelloForBusinessAuthenticationMethod resource type</span></span>

<span data-ttu-id="3ff86-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ff86-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ff86-106">注册到用户的 Windows Hello 企业身份验证方法的表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ff86-106">A representation of a Windows Hello for Business authentication method registered to a user.</span></span> <span data-ttu-id="3ff86-107">Windows Hello 企业应用是 Windows 设备的登录身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="3ff86-107">Windows Hello for Business is a sign-in authentication method for Windows devices.</span></span>

<span data-ttu-id="3ff86-108">继承自 [authenticationMethod](../resources/authenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="3ff86-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3ff86-109">方法</span><span class="sxs-lookup"><span data-stu-id="3ff86-109">Methods</span></span>
|<span data-ttu-id="3ff86-110">方法</span><span class="sxs-lookup"><span data-stu-id="3ff86-110">Method</span></span>|<span data-ttu-id="3ff86-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3ff86-111">Return type</span></span>|<span data-ttu-id="3ff86-112">说明</span><span class="sxs-lookup"><span data-stu-id="3ff86-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3ff86-113">列出 windowsHelloForBusinessAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="3ff86-113">List windowsHelloForBusinessAuthenticationMethods</span></span>](../api/windowshelloforbusinessauthenticationmethod-list.md)|<span data-ttu-id="3ff86-114">[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ff86-114">[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) collection</span></span>|<span data-ttu-id="3ff86-115">获取 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="3ff86-115">Get a list of the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="3ff86-116">获取 windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ff86-116">Get windowsHelloForBusinessAuthenticationMethod</span></span>](../api/windowshelloforbusinessauthenticationmethod-get.md)|[<span data-ttu-id="3ff86-117">windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ff86-117">windowsHelloForBusinessAuthenticationMethod</span></span>](../resources/windowshelloforbusinessauthenticationmethod.md)|<span data-ttu-id="3ff86-118">读取 [windowsHelloForBusinessAuthenticationMethod 对象的属性和](../resources/windowshelloforbusinessauthenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="3ff86-118">Read the properties and relationships of a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="3ff86-119">删除 windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ff86-119">Delete windowsHelloForBusinessAuthenticationMethod</span></span>](../api/windowshelloforbusinessauthenticationmethod-delete.md)|<span data-ttu-id="3ff86-120">无</span><span class="sxs-lookup"><span data-stu-id="3ff86-120">None</span></span>|<span data-ttu-id="3ff86-121">删除 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ff86-121">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ff86-122">属性</span><span class="sxs-lookup"><span data-stu-id="3ff86-122">Properties</span></span>
|<span data-ttu-id="3ff86-123">属性</span><span class="sxs-lookup"><span data-stu-id="3ff86-123">Property</span></span>|<span data-ttu-id="3ff86-124">类型</span><span class="sxs-lookup"><span data-stu-id="3ff86-124">Type</span></span>|<span data-ttu-id="3ff86-125">说明</span><span class="sxs-lookup"><span data-stu-id="3ff86-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ff86-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ff86-126">createdDateTime</span></span>|<span data-ttu-id="3ff86-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ff86-127">DateTimeOffset</span></span>|<span data-ttu-id="3ff86-128">注册此 Windows Hello 企业密钥的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3ff86-128">The date and time that this Windows Hello for Business key was registered.</span></span>|
|<span data-ttu-id="3ff86-129">displayName</span><span class="sxs-lookup"><span data-stu-id="3ff86-129">displayName</span></span>|<span data-ttu-id="3ff86-130">String</span><span class="sxs-lookup"><span data-stu-id="3ff86-130">String</span></span>|<span data-ttu-id="3ff86-131">注册 Windows Hello 企业应用的设备的名称</span><span class="sxs-lookup"><span data-stu-id="3ff86-131">The name of the device on which Windows Hello for Business is registered</span></span>|
|<span data-ttu-id="3ff86-132">id</span><span class="sxs-lookup"><span data-stu-id="3ff86-132">id</span></span>|<span data-ttu-id="3ff86-133">String</span><span class="sxs-lookup"><span data-stu-id="3ff86-133">String</span></span>|<span data-ttu-id="3ff86-134">此身份验证方法的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3ff86-134">A unique identifier for this authentication method.</span></span> <span data-ttu-id="3ff86-135">继承自 [authenticationMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="3ff86-135">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="3ff86-136">keyStrength</span><span class="sxs-lookup"><span data-stu-id="3ff86-136">keyStrength</span></span>|<span data-ttu-id="3ff86-137">authenticationMethodKeyStrength</span><span class="sxs-lookup"><span data-stu-id="3ff86-137">authenticationMethodKeyStrength</span></span>|<span data-ttu-id="3ff86-138">此 Windows Hello 企业密钥的关键强度。</span><span class="sxs-lookup"><span data-stu-id="3ff86-138">Key strength of this Windows Hello for Business key.</span></span> <span data-ttu-id="3ff86-139">可取值为：`normal`、`weak`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="3ff86-139">Possible values are: `normal`, `weak`, `unknown`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ff86-140">关系</span><span class="sxs-lookup"><span data-stu-id="3ff86-140">Relationships</span></span>
|<span data-ttu-id="3ff86-141">关系</span><span class="sxs-lookup"><span data-stu-id="3ff86-141">Relationship</span></span>|<span data-ttu-id="3ff86-142">类型</span><span class="sxs-lookup"><span data-stu-id="3ff86-142">Type</span></span>|<span data-ttu-id="3ff86-143">说明</span><span class="sxs-lookup"><span data-stu-id="3ff86-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ff86-144">设备</span><span class="sxs-lookup"><span data-stu-id="3ff86-144">device</span></span>|[<span data-ttu-id="3ff86-145">设备</span><span class="sxs-lookup"><span data-stu-id="3ff86-145">device</span></span>](../resources/device.md)|<span data-ttu-id="3ff86-146">此 Windows Hello 企业密钥所在的已注册设备。</span><span class="sxs-lookup"><span data-stu-id="3ff86-146">The registered device on which this Windows Hello for Business key resides.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ff86-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ff86-147">JSON representation</span></span>
<span data-ttu-id="3ff86-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ff86-148">The following is a JSON representation of the resource.</span></span>
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
