# vdxf-specifications

This repository specifies naming schemes for general VDXF keys to be used to tag and identify data stored in centralized or decentralized services.  These general keys, when hashed together with a unique VerusID, provide globally unique identifiers that bind the stored data to the VerusID.

VDXF keys are collison-free 20 byte identifiers that correspond to arbitrary URIs.  Systematically defined URIs, such as those specified in this repository, may be used by applications to define and represent any desired data, such as digital art, licenses, legal contracts, social media profiles, social media posts, accreditations, messaging systems, hierarchical naming systems, or anything else.

VerusIDs are friendly-name namespaces that are uniquely registered on the Verus blockchain network.  These namespaces may also be represented by, and correspond to, i-addresses that are globally unique public keys that can be controlled cryptographically using private keys.  The VerusID system provides the ability for users to have permissionless, self-sovereign control of a namespace, including the ability to provide verifiable signatures confirming control over the namespace at any specific point in time.

VerusIDs also contain attached contentmaps which are arbitary key/value stores that can be used to point to arbitrary URIs including to data storage accounts or locations.

The combination of VDXF, VerusIDs and external storage systems that support tagging and indexing provide the ability for users to have permissionless self-sovereign control over an unlimited amount of any type of data, thus enabling any type of permissionless, self sovereign application, without the need for trust or centralized mediators.

The purpose of this repository is to propose systematically defined URIs that support the ability of applications to define and represent specific types of data for applications.

There are generally three types of naming schemes, which correpond to the way in which data is stored and retrieved.

Account-Based Storage - in these, contentmaps will point to storage accounts that may or may not be controlled by the VerusID that is pointing to the account.  Globally unique tags will be searched within the account in order to retrieve the bound data.

Location-Based Storage - this is more specific than account-based storage in that a contentmap points to a specific data location (eg. a specific transaction in arweave).  Bound data will be retrieved directly from the location.

Service-Based Storage - this is less specific than account-based storage.  Here, an application does not consult the contentmap but queries an entire indexed storage service (eg arweave) for the globally unique identifiers that represent the desired data.

