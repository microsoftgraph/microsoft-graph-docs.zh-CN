---
title: certificateBasedAuthConfiguration 资源类型
description: 表示证书颁发机构的集合。
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b37022852407951fb850b8e82508cfff1973247f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161150"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="92651-103">certificateBasedAuthConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="92651-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="92651-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92651-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92651-105">通过基于证书的身份验证，可以在将 Exchange Online 帐户连接到：Windows、Android 或 iOS 设备上，通过 Azure Active Directory 通过客户端证书进行身份验证：</span><span class="sxs-lookup"><span data-stu-id="92651-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="92651-106">Microsoft 移动应用程序，如 Outlook 和 Word</span><span class="sxs-lookup"><span data-stu-id="92651-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="92651-107">Exchange ActiveSync (EAS) 客户端</span><span class="sxs-lookup"><span data-stu-id="92651-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="92651-108">配置此功能无需将用户名和密码组合输入到移动设备上的某些邮件Microsoft Office应用程序。</span><span class="sxs-lookup"><span data-stu-id="92651-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="92651-109">基于证书的身份验证配置通过证书颁发机构集合提供。</span><span class="sxs-lookup"><span data-stu-id="92651-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="92651-110">证书颁发机构用于建立受信任的证书链，使客户端可以通过 Azure Active Directory 使用客户端证书进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="92651-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="92651-111">详细了解 Azure [Active Directory 中基于证书的身份验证](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)。</span><span class="sxs-lookup"><span data-stu-id="92651-111">Learn more about [certificate-based authentication in Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="92651-112">方法</span><span class="sxs-lookup"><span data-stu-id="92651-112">Methods</span></span>

| <span data-ttu-id="92651-113">方法</span><span class="sxs-lookup"><span data-stu-id="92651-113">Method</span></span>       | <span data-ttu-id="92651-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="92651-114">Return Type</span></span> | <span data-ttu-id="92651-115">说明</span><span class="sxs-lookup"><span data-stu-id="92651-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="92651-116">列出 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="92651-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="92651-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="92651-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="92651-118">列出 **certificateBasedAuthConfiguration** 集合的属性。</span><span class="sxs-lookup"><span data-stu-id="92651-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="92651-119">获取 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="92651-119">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="92651-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="92651-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="92651-121">读取 **certificateBasedAuthConfiguration 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="92651-121">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="92651-122">创建 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="92651-122">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="92651-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="92651-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="92651-124">创建新的 **certificateBasedAuthConfiguration** 对象。</span><span class="sxs-lookup"><span data-stu-id="92651-124">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="92651-125">删除 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="92651-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="92651-126">无</span><span class="sxs-lookup"><span data-stu-id="92651-126">None</span></span> | <span data-ttu-id="92651-127">删除 **certificateBasedAuthConfiguration** 对象。</span><span class="sxs-lookup"><span data-stu-id="92651-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="92651-128">不支持更新 cerficateBasedAuthConfiguration。</span><span class="sxs-lookup"><span data-stu-id="92651-128">Updating cerficateBasedAuthConfiguration is not supported.</span></span> <span data-ttu-id="92651-129">若要更改 cerficateBasedAuthConfiguration，请首先删除并创建新的 cerficateBasedAuthConfiguration。</span><span class="sxs-lookup"><span data-stu-id="92651-129">To change a cerficateBasedAuthConfiguration, first delete and then create a new cerficateBasedAuthConfiguration.</span></span>

## <a name="properties"></a><span data-ttu-id="92651-130">属性</span><span class="sxs-lookup"><span data-stu-id="92651-130">Properties</span></span>

| <span data-ttu-id="92651-131">属性</span><span class="sxs-lookup"><span data-stu-id="92651-131">Property</span></span>     | <span data-ttu-id="92651-132">类型</span><span class="sxs-lookup"><span data-stu-id="92651-132">Type</span></span>        | <span data-ttu-id="92651-133">说明</span><span class="sxs-lookup"><span data-stu-id="92651-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="92651-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="92651-134">certificateAuthorities</span></span>|<span data-ttu-id="92651-135">[certificateAuthority](certificateauthority.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92651-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="92651-136">创建受信任证书链的证书颁发机构的集合。</span><span class="sxs-lookup"><span data-stu-id="92651-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="92651-137">id</span><span class="sxs-lookup"><span data-stu-id="92651-137">id</span></span>|<span data-ttu-id="92651-138">String</span><span class="sxs-lookup"><span data-stu-id="92651-138">String</span></span>|<span data-ttu-id="92651-139">基于证书的身份验证配置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="92651-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="92651-140">只读。</span><span class="sxs-lookup"><span data-stu-id="92651-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92651-141">关系</span><span class="sxs-lookup"><span data-stu-id="92651-141">Relationships</span></span>

<span data-ttu-id="92651-142">无</span><span class="sxs-lookup"><span data-stu-id="92651-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92651-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92651-143">JSON representation</span></span>

<span data-ttu-id="92651-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92651-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "keyProperty": "id"
}-->

```json
{
  "certificateAuthorities": {"@odata.type": "collection(microsoft.graph.certificateAuthority)"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateBasedAuthConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->