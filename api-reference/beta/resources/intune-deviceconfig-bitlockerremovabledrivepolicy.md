---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
author: tfitzmac
ms.openlocfilehash: 15de11384195350b455cd4696a260aedf1de7a26
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354031"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="37317-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="37317-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="37317-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="37317-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37317-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="37317-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37317-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="37317-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37317-107">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="37317-107">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="37317-108">属性</span><span class="sxs-lookup"><span data-stu-id="37317-108">Properties</span></span>
|<span data-ttu-id="37317-109">属性</span><span class="sxs-lookup"><span data-stu-id="37317-109">Property</span></span>|<span data-ttu-id="37317-110">类型</span><span class="sxs-lookup"><span data-stu-id="37317-110">Type</span></span>|<span data-ttu-id="37317-111">说明</span><span class="sxs-lookup"><span data-stu-id="37317-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37317-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="37317-112">encryptionMethod</span></span>|[<span data-ttu-id="37317-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="37317-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="37317-114">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="37317-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="37317-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="37317-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="37317-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="37317-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="37317-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="37317-117">Boolean</span></span>|<span data-ttu-id="37317-118">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="37317-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="37317-119">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="37317-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="37317-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="37317-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="37317-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="37317-121">Boolean</span></span>|<span data-ttu-id="37317-122">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="37317-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37317-123">关系</span><span class="sxs-lookup"><span data-stu-id="37317-123">Relationships</span></span>
<span data-ttu-id="37317-124">无</span><span class="sxs-lookup"><span data-stu-id="37317-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37317-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37317-125">JSON Representation</span></span>
<span data-ttu-id="37317-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37317-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```





