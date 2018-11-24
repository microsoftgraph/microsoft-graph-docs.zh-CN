# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="6c89a-101">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c89a-101">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="6c89a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6c89a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c89a-103">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="6c89a-103">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="6c89a-104">属性</span><span class="sxs-lookup"><span data-stu-id="6c89a-104">Properties</span></span>
|<span data-ttu-id="6c89a-105">属性</span><span class="sxs-lookup"><span data-stu-id="6c89a-105">Property</span></span>|<span data-ttu-id="6c89a-106">类型</span><span class="sxs-lookup"><span data-stu-id="6c89a-106">Type</span></span>|<span data-ttu-id="6c89a-107">说明</span><span class="sxs-lookup"><span data-stu-id="6c89a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c89a-108">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="6c89a-108">encryptionMethod</span></span>|[<span data-ttu-id="6c89a-109">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="6c89a-109">bitLockerEncryptionMethod</span></span>](../resources/intune_deviceconfig_bitlockerencryptionmethod.md)|<span data-ttu-id="6c89a-110">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="6c89a-110">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="6c89a-111">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="6c89a-111">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="6c89a-112">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="6c89a-112">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="6c89a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c89a-113">Boolean</span></span>|<span data-ttu-id="6c89a-114">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="6c89a-114">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="6c89a-115">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="6c89a-115">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="6c89a-116">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="6c89a-116">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="6c89a-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c89a-117">Boolean</span></span>|<span data-ttu-id="6c89a-118">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="6c89a-118">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c89a-119">关系</span><span class="sxs-lookup"><span data-stu-id="6c89a-119">Relationships</span></span>
<span data-ttu-id="6c89a-120">无</span><span class="sxs-lookup"><span data-stu-id="6c89a-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6c89a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c89a-121">JSON Representation</span></span>
<span data-ttu-id="6c89a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c89a-122">Here is a JSON representation of the resource.</span></span>
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



